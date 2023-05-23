# Comparing `tmp/mdninja-1.0.1.tar.gz` & `tmp/mdninja-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mdninja-1.0.1.tar", last modified: Wed Nov 15 14:04:49 2017, max compression
+gzip compressed data, was "mdninja-1.0.2.tar", last modified: Tue May 23 14:49:40 2023, max compression
```

## Comparing `mdninja-1.0.1.tar` & `mdninja-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 pgowda     (501) staff       (20)        0 2017-11-15 14:04:49.000000 mdninja-1.0.1/
-drwxr-xr-x   0 pgowda     (501) staff       (20)        0 2017-11-15 14:04:49.000000 mdninja-1.0.1/mdninja/
--rw-r--r--   0 pgowda     (501) staff       (20)     2079 2017-11-15 14:02:21.000000 mdninja-1.0.1/mdninja/__init__.py
-drwxr-xr-x   0 pgowda     (501) staff       (20)        0 2017-11-15 14:04:49.000000 mdninja-1.0.1/mdninja/templates/
--rw-r--r--   0 pgowda     (501) staff       (20)      311 2017-11-15 13:43:42.000000 mdninja-1.0.1/mdninja/templates/default.html
-drwxr-xr-x   0 pgowda     (501) staff       (20)        0 2017-11-15 14:04:49.000000 mdninja-1.0.1/mdninja.egg-info/
--rw-r--r--   0 pgowda     (501) staff       (20)        1 2017-11-15 14:04:48.000000 mdninja-1.0.1/mdninja.egg-info/dependency_links.txt
--rw-r--r--   0 pgowda     (501) staff       (20)       42 2017-11-15 14:04:48.000000 mdninja-1.0.1/mdninja.egg-info/entry_points.txt
--rw-r--r--   0 pgowda     (501) staff       (20)     2167 2017-11-15 14:04:48.000000 mdninja-1.0.1/mdninja.egg-info/PKG-INFO
--rw-r--r--   0 pgowda     (501) staff       (20)       22 2017-11-15 14:04:48.000000 mdninja-1.0.1/mdninja.egg-info/requires.txt
--rw-r--r--   0 pgowda     (501) staff       (20)      258 2017-11-15 14:04:48.000000 mdninja-1.0.1/mdninja.egg-info/SOURCES.txt
--rw-r--r--   0 pgowda     (501) staff       (20)        8 2017-11-15 14:04:48.000000 mdninja-1.0.1/mdninja.egg-info/top_level.txt
--rw-r--r--   0 pgowda     (501) staff       (20)     2167 2017-11-15 14:04:49.000000 mdninja-1.0.1/PKG-INFO
--rw-r--r--   0 pgowda     (501) staff       (20)      945 2017-11-15 04:20:51.000000 mdninja-1.0.1/README.rst
--rw-r--r--   0 pgowda     (501) staff       (20)       38 2017-11-15 14:04:49.000000 mdninja-1.0.1/setup.cfg
--rw-r--r--   0 pgowda     (501) staff       (20)     1704 2017-11-15 13:43:56.000000 mdninja-1.0.1/setup.py
+drwxr-xr-x   0 pradeep    (501) staff       (20)        0 2023-05-23 14:49:40.143373 mdninja-1.0.2/
+-rw-r--r--   0 pradeep    (501) staff       (20)     1606 2023-05-23 14:49:40.143223 mdninja-1.0.2/PKG-INFO
+-rw-r--r--   0 pradeep    (501) staff       (20)      945 2023-05-22 17:25:08.000000 mdninja-1.0.2/README.rst
+drwxr-xr-x   0 pradeep    (501) staff       (20)        0 2023-05-23 14:49:40.141579 mdninja-1.0.2/mdninja/
+-rw-r--r--   0 pradeep    (501) staff       (20)     2079 2023-05-22 17:25:08.000000 mdninja-1.0.2/mdninja/__init__.py
+drwxr-xr-x   0 pradeep    (501) staff       (20)        0 2023-05-23 14:49:40.142837 mdninja-1.0.2/mdninja/templates/
+-rw-r--r--   0 pradeep    (501) staff       (20)      311 2023-05-22 17:25:08.000000 mdninja-1.0.2/mdninja/templates/default.html
+drwxr-xr-x   0 pradeep    (501) staff       (20)        0 2023-05-23 14:49:40.142702 mdninja-1.0.2/mdninja.egg-info/
+-rw-r--r--   0 pradeep    (501) staff       (20)     1606 2023-05-23 14:49:40.000000 mdninja-1.0.2/mdninja.egg-info/PKG-INFO
+-rw-r--r--   0 pradeep    (501) staff       (20)      258 2023-05-23 14:49:40.000000 mdninja-1.0.2/mdninja.egg-info/SOURCES.txt
+-rw-r--r--   0 pradeep    (501) staff       (20)        1 2023-05-23 14:49:40.000000 mdninja-1.0.2/mdninja.egg-info/dependency_links.txt
+-rw-r--r--   0 pradeep    (501) staff       (20)       41 2023-05-23 14:49:40.000000 mdninja-1.0.2/mdninja.egg-info/entry_points.txt
+-rw-r--r--   0 pradeep    (501) staff       (20)       22 2023-05-23 14:49:40.000000 mdninja-1.0.2/mdninja.egg-info/requires.txt
+-rw-r--r--   0 pradeep    (501) staff       (20)        8 2023-05-23 14:49:40.000000 mdninja-1.0.2/mdninja.egg-info/top_level.txt
+-rw-r--r--   0 pradeep    (501) staff       (20)       38 2023-05-23 14:49:40.143417 mdninja-1.0.2/setup.cfg
+-rw-r--r--   0 pradeep    (501) staff       (20)     1703 2023-05-23 01:39:03.000000 mdninja-1.0.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `mdninja-1.0.1/mdninja/__init__.py` & `mdninja-1.0.2/mdninja/__init__.py`

 * *Files identical despite different names*

### Comparing `mdninja-1.0.1/mdninja.egg-info/PKG-INFO` & `mdninja-1.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,83 +1,81 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: mdninja
-Version: 1.0.1
+Version: 1.0.2
 Summary: mdninja + markdown + jinja2 = beautiful HTML
 Home-page: https://github.com/btbytes/mdninja
 Author: Pradeep Gowda
 Author-email: btbytes+mdninja@gmail.com
 License: MIT
-Description-Content-Type: UNKNOWN
-Description: =======
-        mdninja
-        =======
-        
-        **mdninja + markdown + jinja2 = beautiful HTML documents**
-        
-        `mdninja` is a document processor that converts markdown documents into HTML document by applying Jinja2 templating.
-        
-        Installation
-        ------------
-        
-        ::
-        
-          pip install mdninja
-        
-        Usage
-        -----
-        
-        Simple use:
-        
-        ::
-        
-          mdninja doc.md -o doc.html
-        
-        
-        If you want to use a different template:
-        
-        ::
-        
-          mdninja doc.md -o doc.html --template=stylish.html
-        
-        
-        The default template is:
-        
-        ::
-        
-        	<!DOCTYPE html>
-        	<html>
-        		<head>
-        			<title>{% for title in meta.title %}{{title}} {% endfor %}</title>
-        		</head>
-        		<body>
-        			<h1>{% for title in meta.title %}{{title}} {% endfor %}</h1>
-        			{{ body }}
-        			<hr/>
-        		</body>
-        	</html>
-        
-        Metadata (like `title` above) is added to the document by adding metadata headers like this at the top of the file
-        
-        ::
-        
-          Title: A simple document
-        
-        
-        Alternatively, you can specify the meatadata using a YAML style header too:
-        
-        ::
-        
-        	---
-        	title: A simple document
-        	---
-        
 Keywords: markdown jinja2 publishing
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
-Requires-Python: ~=3.4
+Requires-Python: ~=3.9
+
+=======
+mdninja
+=======
+
+**mdninja + markdown + jinja2 = beautiful HTML documents**
+
+`mdninja` is a document processor that converts markdown documents into HTML document by applying Jinja2 templating.
+
+Installation
+------------
+
+::
+
+  pip install mdninja
+
+Usage
+-----
+
+Simple use:
+
+::
+
+  mdninja doc.md -o doc.html
+
+
+If you want to use a different template:
+
+::
+
+  mdninja doc.md -o doc.html --template=stylish.html
+
+
+The default template is:
+
+::
+
+	<!DOCTYPE html>
+	<html>
+		<head>
+			<title>{% for title in meta.title %}{{title}} {% endfor %}</title>
+		</head>
+		<body>
+			<h1>{% for title in meta.title %}{{title}} {% endfor %}</h1>
+			{{ body }}
+			<hr/>
+		</body>
+	</html>
+
+Metadata (like `title` above) is added to the document by adding metadata headers like this at the top of the file
+
+::
+
+  Title: A simple document
+
+
+Alternatively, you can specify the meatadata using a YAML style header too:
+
+::
+
+	---
+	title: A simple document
+	---
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 1.2 Name: mdninja Version: 1.0.1 Summary: mdninja + markdown
+Metadata-Version: 2.1 Name: mdninja Version: 1.0.2 Summary: mdninja + markdown
 + jinja2 = beautiful HTML Home-page: https://github.com/btbytes/mdninja Author:
-Pradeep Gowda Author-email: btbytes+mdninja@gmail.com License: MIT Description-
-Content-Type: UNKNOWN Description: ======= mdninja ======= **mdninja + markdown
-+ jinja2 = beautiful HTML documents** `mdninja` is a document processor that
-converts markdown documents into HTML document by applying Jinja2 templating.
-Installation ------------ :: pip install mdninja Usage ----- Simple use: ::
-mdninja doc.md -o doc.html If you want to use a different template: :: mdninja
-doc.md -o doc.html --template=stylish.html The default template is: ::
+Pradeep Gowda Author-email: btbytes+mdninja@gmail.com License: MIT Keywords:
+markdown jinja2 publishing Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: End Users/Desktop Classifier: Topic ::
+Utilities Classifier: License :: OSI Approved :: MIT License Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.3 Classifier: Programming Language :: Python :: 3.4 Classifier:
+Programming Language :: Python :: 3.5 Requires-Python: ~=3.9 ======= mdninja
+======= **mdninja + markdown + jinja2 = beautiful HTML documents** `mdninja` is
+a document processor that converts markdown documents into HTML document by
+applying Jinja2 templating. Installation ------------ :: pip install mdninja
+Usage ----- Simple use: :: mdninja doc.md -o doc.html If you want to use a
+different template: :: mdninja doc.md -o doc.html --template=stylish.html The
+default template is: ::
 ****** {% for title in meta.title %}{{title}} {% endfor %} ******
 {{ body }}
 ===============================================================================
 Metadata (like `title` above) is added to the document by adding metadata
 headers like this at the top of the file :: Title: A simple document
 Alternatively, you can specify the meatadata using a YAML style header too: ::
---- title: A simple document --- Keywords: markdown jinja2 publishing Platform:
-UNKNOWN Classifier: Development Status :: 4 - Beta Classifier: Intended
-Audience :: End Users/Desktop Classifier: Topic :: Utilities Classifier:
-License :: OSI Approved :: MIT License Classifier: Programming Language ::
-Python :: 3 Classifier: Programming Language :: Python :: 3.3 Classifier:
-Programming Language :: Python :: 3.4 Classifier: Programming Language ::
-Python :: 3.5 Requires-Python: ~=3.4
+--- title: A simple document ---
```

### Comparing `mdninja-1.0.1/PKG-INFO` & `mdninja-1.0.2/mdninja.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,83 +1,81 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: mdninja
-Version: 1.0.1
+Version: 1.0.2
 Summary: mdninja + markdown + jinja2 = beautiful HTML
 Home-page: https://github.com/btbytes/mdninja
 Author: Pradeep Gowda
 Author-email: btbytes+mdninja@gmail.com
 License: MIT
-Description-Content-Type: UNKNOWN
-Description: =======
-        mdninja
-        =======
-        
-        **mdninja + markdown + jinja2 = beautiful HTML documents**
-        
-        `mdninja` is a document processor that converts markdown documents into HTML document by applying Jinja2 templating.
-        
-        Installation
-        ------------
-        
-        ::
-        
-          pip install mdninja
-        
-        Usage
-        -----
-        
-        Simple use:
-        
-        ::
-        
-          mdninja doc.md -o doc.html
-        
-        
-        If you want to use a different template:
-        
-        ::
-        
-          mdninja doc.md -o doc.html --template=stylish.html
-        
-        
-        The default template is:
-        
-        ::
-        
-        	<!DOCTYPE html>
-        	<html>
-        		<head>
-        			<title>{% for title in meta.title %}{{title}} {% endfor %}</title>
-        		</head>
-        		<body>
-        			<h1>{% for title in meta.title %}{{title}} {% endfor %}</h1>
-        			{{ body }}
-        			<hr/>
-        		</body>
-        	</html>
-        
-        Metadata (like `title` above) is added to the document by adding metadata headers like this at the top of the file
-        
-        ::
-        
-          Title: A simple document
-        
-        
-        Alternatively, you can specify the meatadata using a YAML style header too:
-        
-        ::
-        
-        	---
-        	title: A simple document
-        	---
-        
 Keywords: markdown jinja2 publishing
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
-Requires-Python: ~=3.4
+Requires-Python: ~=3.9
+
+=======
+mdninja
+=======
+
+**mdninja + markdown + jinja2 = beautiful HTML documents**
+
+`mdninja` is a document processor that converts markdown documents into HTML document by applying Jinja2 templating.
+
+Installation
+------------
+
+::
+
+  pip install mdninja
+
+Usage
+-----
+
+Simple use:
+
+::
+
+  mdninja doc.md -o doc.html
+
+
+If you want to use a different template:
+
+::
+
+  mdninja doc.md -o doc.html --template=stylish.html
+
+
+The default template is:
+
+::
+
+	<!DOCTYPE html>
+	<html>
+		<head>
+			<title>{% for title in meta.title %}{{title}} {% endfor %}</title>
+		</head>
+		<body>
+			<h1>{% for title in meta.title %}{{title}} {% endfor %}</h1>
+			{{ body }}
+			<hr/>
+		</body>
+	</html>
+
+Metadata (like `title` above) is added to the document by adding metadata headers like this at the top of the file
+
+::
+
+  Title: A simple document
+
+
+Alternatively, you can specify the meatadata using a YAML style header too:
+
+::
+
+	---
+	title: A simple document
+	---
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 1.2 Name: mdninja Version: 1.0.1 Summary: mdninja + markdown
+Metadata-Version: 2.1 Name: mdninja Version: 1.0.2 Summary: mdninja + markdown
 + jinja2 = beautiful HTML Home-page: https://github.com/btbytes/mdninja Author:
-Pradeep Gowda Author-email: btbytes+mdninja@gmail.com License: MIT Description-
-Content-Type: UNKNOWN Description: ======= mdninja ======= **mdninja + markdown
-+ jinja2 = beautiful HTML documents** `mdninja` is a document processor that
-converts markdown documents into HTML document by applying Jinja2 templating.
-Installation ------------ :: pip install mdninja Usage ----- Simple use: ::
-mdninja doc.md -o doc.html If you want to use a different template: :: mdninja
-doc.md -o doc.html --template=stylish.html The default template is: ::
+Pradeep Gowda Author-email: btbytes+mdninja@gmail.com License: MIT Keywords:
+markdown jinja2 publishing Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: End Users/Desktop Classifier: Topic ::
+Utilities Classifier: License :: OSI Approved :: MIT License Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.3 Classifier: Programming Language :: Python :: 3.4 Classifier:
+Programming Language :: Python :: 3.5 Requires-Python: ~=3.9 ======= mdninja
+======= **mdninja + markdown + jinja2 = beautiful HTML documents** `mdninja` is
+a document processor that converts markdown documents into HTML document by
+applying Jinja2 templating. Installation ------------ :: pip install mdninja
+Usage ----- Simple use: :: mdninja doc.md -o doc.html If you want to use a
+different template: :: mdninja doc.md -o doc.html --template=stylish.html The
+default template is: ::
 ****** {% for title in meta.title %}{{title}} {% endfor %} ******
 {{ body }}
 ===============================================================================
 Metadata (like `title` above) is added to the document by adding metadata
 headers like this at the top of the file :: Title: A simple document
 Alternatively, you can specify the meatadata using a YAML style header too: ::
---- title: A simple document --- Keywords: markdown jinja2 publishing Platform:
-UNKNOWN Classifier: Development Status :: 4 - Beta Classifier: Intended
-Audience :: End Users/Desktop Classifier: Topic :: Utilities Classifier:
-License :: OSI Approved :: MIT License Classifier: Programming Language ::
-Python :: 3 Classifier: Programming Language :: Python :: 3.3 Classifier:
-Programming Language :: Python :: 3.4 Classifier: Programming Language ::
-Python :: 3.5 Requires-Python: ~=3.4
+--- title: A simple document ---
```

### Comparing `mdninja-1.0.1/README.rst` & `mdninja-1.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `mdninja-1.0.1/setup.py` & `mdninja-1.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,51 +5,51 @@
 
 from setuptools import setup, find_packages
 from codecs import open
 from os import path
 
 here = path.abspath(path.dirname(__file__))
 
-with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
+with open(path.join(here, "README.rst"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
-    name='mdninja',
-    version='1.0.1',
-    description='mdninja + markdown + jinja2 = beautiful HTML',
+    name="mdninja",
+    version="1.0.2",
+    description="mdninja + markdown + jinja2 = beautiful HTML",
     long_description=long_description,
-    url='https://github.com/btbytes/mdninja',
-    author='Pradeep Gowda',
-    author_email='btbytes+mdninja@gmail.com',
-    license='MIT',
+    url="https://github.com/btbytes/mdninja",
+    author="Pradeep Gowda",
+    author_email="btbytes+mdninja@gmail.com",
+    license="MIT",
     # See https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
-        'Development Status :: 4 - Beta',
-        'Intended Audience :: End Users/Desktop',
-        'Topic :: Utilities',
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.3',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
+        "Development Status :: 4 - Beta",
+        "Intended Audience :: End Users/Desktop",
+        "Topic :: Utilities",
+        "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.3",
+        "Programming Language :: Python :: 3.4",
+        "Programming Language :: Python :: 3.5",
     ],
-    keywords='markdown jinja2 publishing',
-    packages=find_packages(exclude=['contrib', 'docs', 'tests']),
-    python_requires='~=3.4',
-    install_requires=['markdown', 'jinja2', 'click'],
-
+    keywords="markdown jinja2 publishing",
+    packages=find_packages(exclude=["contrib", "docs", "tests"]),
+    python_requires="~=3.9",
+    install_requires=["markdown", "jinja2", "click"],
     # List additional groups of dependencies here (e.g. development
     # dependencies). You can install these using the following syntax,
     # for example:
     # $ pip install -e .[dev,test]
     # extras_require={
     #    'dev': ['check-manifest'],
     #    'test': ['coverage'],
     # },
     package_data={
-        'mdninja': ['templates/default.html'],
+        "mdninja": ["templates/default.html"],
     },
     entry_points={
-        'console_scripts': [
-            'mdninja=mdninja:main',
+        "console_scripts": [
+            "mdninja=mdninja:main",
         ],
-    }, )
+    },
+)
```

