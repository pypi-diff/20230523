# Comparing `tmp/SIOTCommon-0.1.2.tar.gz` & `tmp/SIOTCommon-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SIOTCommon-0.1.2.tar", last modified: Mon May 22 22:46:36 2023, max compression
+gzip compressed data, was "SIOTCommon-0.1.3.tar", last modified: Mon May 22 23:18:59 2023, max compression
```

## Comparing `SIOTCommon-0.1.2.tar` & `SIOTCommon-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 22:46:36.530639 SIOTCommon-0.1.2/
--rw-rw-rw-   0        0        0      339 2023-05-22 22:46:36.530639 SIOTCommon-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-11 20:29:38.000000 SIOTCommon-0.1.2/README.txt
-drwxrwxrwx   0        0        0        0 2023-05-22 22:46:36.519639 SIOTCommon-0.1.2/SIOTC/
--rw-rw-rw-   0        0        0     2080 2023-05-22 22:40:04.000000 SIOTCommon-0.1.2/SIOTC/DatabaseLayer.py
--rw-rw-rw-   0        0        0    11682 2023-05-22 22:45:01.000000 SIOTCommon-0.1.2/SIOTC/Operations.py
--rw-rw-rw-   0        0        0      484 2023-04-20 13:32:21.000000 SIOTCommon-0.1.2/SIOTC/__init__.py
--rw-rw-rw-   0        0        0     2738 2023-05-05 13:45:10.000000 SIOTCommon-0.1.2/SIOTC/helperhttps.py
-drwxrwxrwx   0        0        0        0 2023-05-22 22:46:36.528670 SIOTCommon-0.1.2/SIOTCommon.egg-info/
--rw-rw-rw-   0        0        0      339 2023-05-22 22:46:36.000000 SIOTCommon-0.1.2/SIOTCommon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-05-22 22:46:36.000000 SIOTCommon-0.1.2/SIOTCommon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 22:46:36.000000 SIOTCommon-0.1.2/SIOTCommon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      636 2023-05-22 22:46:36.000000 SIOTCommon-0.1.2/SIOTCommon.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-22 22:46:36.000000 SIOTCommon-0.1.2/SIOTCommon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 22:46:36.531636 SIOTCommon-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      581 2023-05-22 22:46:30.000000 SIOTCommon-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 23:18:59.698311 SIOTCommon-0.1.3/
+-rw-rw-rw-   0        0        0      339 2023-05-22 23:18:59.697311 SIOTCommon-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-04-11 20:29:38.000000 SIOTCommon-0.1.3/README.txt
+drwxrwxrwx   0        0        0        0 2023-05-22 23:18:59.688308 SIOTCommon-0.1.3/SIOTC/
+-rw-rw-rw-   0        0        0     2374 2023-05-22 23:17:55.000000 SIOTCommon-0.1.3/SIOTC/DatabaseLayer.py
+-rw-rw-rw-   0        0        0    11682 2023-05-22 22:45:01.000000 SIOTCommon-0.1.3/SIOTC/Operations.py
+-rw-rw-rw-   0        0        0      484 2023-04-20 13:32:21.000000 SIOTCommon-0.1.3/SIOTC/__init__.py
+-rw-rw-rw-   0        0        0     2738 2023-05-05 13:45:10.000000 SIOTCommon-0.1.3/SIOTC/helperhttps.py
+drwxrwxrwx   0        0        0        0 2023-05-22 23:18:59.696308 SIOTCommon-0.1.3/SIOTCommon.egg-info/
+-rw-rw-rw-   0        0        0      339 2023-05-22 23:18:59.000000 SIOTCommon-0.1.3/SIOTCommon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-05-22 23:18:59.000000 SIOTCommon-0.1.3/SIOTCommon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 23:18:59.000000 SIOTCommon-0.1.3/SIOTCommon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      636 2023-05-22 23:18:59.000000 SIOTCommon-0.1.3/SIOTCommon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-22 23:18:59.000000 SIOTCommon-0.1.3/SIOTCommon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 23:18:59.699329 SIOTCommon-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      581 2023-05-22 23:18:50.000000 SIOTCommon-0.1.3/setup.py
```

### Comparing `SIOTCommon-0.1.2/SIOTC/DatabaseLayer.py` & `SIOTCommon-0.1.3/SIOTC/DatabaseLayer.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,20 +7,33 @@
 filename = 'db_config.txt'
 file_path = os.path.join(dir_path, filename)
 
 with open(file_path, 'r') as f:
     # Write the connection string to the file
     first_line = f.readline()
 
+global_session = None
+
 def GetSession():
+    global global_session
+
+    # Check if a session already exists
+    if global_session is not None:
+        return global_session
+
+    # Create a new session if it doesn't exist
     Base = automap_base()
     engine = create_engine(first_line, echo=True)
     Base.prepare(engine, reflect=True, schema='public')
     session_factory = sessionmaker(bind=engine)
     session = scoped_session(session_factory)
+
+    # Store the session in the global variable
+    global_session = session
+
     return session, Base
 
 def GetModel(table_name):
     session, Base = GetSession()
     table_model = getattr(Base.classes, table_name, None)
     if table_model is None:
         raise ValueError(f"Table model not found for table name: {table_name}")
```

### Comparing `SIOTCommon-0.1.2/SIOTC/Operations.py` & `SIOTCommon-0.1.3/SIOTC/Operations.py`

 * *Files identical despite different names*

### Comparing `SIOTCommon-0.1.2/SIOTC/helperhttps.py` & `SIOTCommon-0.1.3/SIOTC/helperhttps.py`

 * *Files identical despite different names*

### Comparing `SIOTCommon-0.1.2/SIOTCommon.egg-info/requires.txt` & `SIOTCommon-0.1.3/SIOTCommon.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `SIOTCommon-0.1.2/setup.py` & `SIOTCommon-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='SIOTCommon',
-    version='0.1.2',
+    version='0.1.3',
     packages=find_packages(),
     install_requires=requirements,
     author='Anton Persson',
     author_email='Antonnilspersson@gmail.com',
     description='Common operations for sweiot microservices',
     url='https://github.com/AntonNPersson/SweIoTServices.git',
     classifiers=[
```

